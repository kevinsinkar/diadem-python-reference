---
title: "IRepD3CurveListInt.Item"
description: "Returns the curve of a 3D axis system associated with a specific name or index, in DIAdem REPORT."
---

# IRepD3CurveListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for 3DCurves

Returns the curve of a 3D axis system associated with a specific name or index, in DIAdem REPORT.

## Signature

```python
return_value = obj.Item(NameOrIndex)
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
oMy3DCurves = oMy3DAxisSystem.Curves3D
oMy3DCurves.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMy3DCurves(1).Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurves(1).Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurves(1).Shape.ZChannel.Reference = "[2]/[3]"
oMy3DCurves(1).Shape.DataStructure = dd.e3DDataStructureMatrix
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepD3CurveListInt.htm`*
