---
title: "IRepD2SelectedSubObjectsListInt.Add2D"
description: "Selects the subobject of a 2D axis system in DIAdem REPORT associated with a specific index."
---

# IRepD2SelectedSubObjectsListInt.Add2D

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add2D for 2DSelectedElements

Selects the subobject of a 2D axis system in DIAdem REPORT associated with a specific index.

## Signature

```python
return_value = obj.Add2D(ElementType, Index)
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
dd.Report.Refresh()
oMy2DAxisSystem.SelectedElements.Add2D(dd.e2DElementYAxis, 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add2D_IRepD2SelectedSubObjectsListInt.htm`*
