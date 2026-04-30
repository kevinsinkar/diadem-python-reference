---
title: "IRepD3SelectedSubObjectsListInt.Add3D"
description: "Selects the subobject of a 3D axis system in DIAdem REPORT associated with a specific index."
---

# IRepD3SelectedSubObjectsListInt.Add3D

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add3D for 3DSelectedElements

Selects the subobject of a 3D axis system in DIAdem REPORT associated with a specific index.

## Signature

```python
return_value = obj.Add3D(ElementType, Index)
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapePoints, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.Settings.Marker.Type = dd.eMarkerAsterisk
dd.Report.Refresh()
oMy3DAxisSystem.SelectedElements.Add3D(dd.e3DElementYAxis, 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add3D_IRepD3SelectedSubObjectsListInt.htm`*
