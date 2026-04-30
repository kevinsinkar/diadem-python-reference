---
title: "IRepPolarCurveListInt.ChangeShape"
description: "Changes the display mode of a curve in a polar axis system in DIAdem REPORT."
---

# IRepPolarCurveListInt.ChangeShape

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ChangeShape for PolarCurves

Changes the display mode of a curve in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.ChangeShape(NameOrIndex, ShapeType)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePolarShapeLine` | 0 | Line |
| `ePolarShapeLineAndPoints` | 1 | Line and points |
| `ePolarShapeSpikes` | 2 | Spikes |
| `ePolarShapeDifferential` | 3 | Differential |

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyAxisSystem")
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
dd.Report.Refresh()
dd.Pause(5)
oMyPolarAxisSystem.CurvesPolar.ChangeShape("MyCurve",dd.e2DShapeSpikes)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ChangeShape_IRepPolarCurveListInt.htm`*
