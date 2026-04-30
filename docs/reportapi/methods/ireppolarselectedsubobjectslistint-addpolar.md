---
title: "IRepPolarSelectedSubObjectsListInt.AddPolar"
description: "Selects the subobject of a polar axis system in DIAdem REPORT associated with a specific index."
---

# IRepPolarSelectedSubObjectsListInt.AddPolar

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: AddPolar for PolarSelectedElements

Selects the subobject of a polar axis system in DIAdem REPORT associated with a specific index.

## Signature

```python
return_value = obj.AddPolar(ElementType, Index)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePolarElementRadialAxis` | 0 | Radial axis |
| `ePolarElementRadialAxisNumbers` | 1 | Radial axis scale |
| `ePolarElementRadialAxisLabel` | 2 | Radial axis label |
| `ePolarElementSectorNumbers` | 3 | Circle scale |
| `ePolarElementCurve` | 4 | Curve |
| `ePolarElementCurveLegend` | 5 | Legend |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
oMyPolarAxisSystem.SelectedElements.AddPolar(dd.ePolarElementRadialAxisLabel, 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_AddPolar_IRepPolarSelectedSubObjectsListInt.htm`*
