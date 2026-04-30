---
title: "IRepD3PaletteColoredLineListInt.Item"
description: "Returns the line properties associated with a specific index of the color areas defined in the color palette for the Palette line color in a 3D axis system in D"
---

# IRepD3PaletteColoredLineListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for 3DPaletteColoredLines

Returns the line properties associated with a specific index of the color areas defined in the color palette for the Palette line color in a 3D axis system in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.DataStructure = dd.e3DDataStructureMatrix

oMySurfaceLine = oMy3DCurve.Shape.Extensions.SurfaceIsoline
oMySurfaceLine.DisplayType = dd.e3DIsolineCorrespondingToIsoValueAndProjected
oMySurfaceLine.Visible = True
oMySurfaceLine.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColoredLines = oMy3DCurve.Shape.Settings.Palette
for i in range( 1, oMyColoredLines.Count+1):
    oMyColoredLines(i).LineType = dd.eLineTypeDashDot
    oMyColoredLines(i).Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepD3PaletteColoredLineListInt.htm`*
