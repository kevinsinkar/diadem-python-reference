---
title: "IRepPolarRadialAxisInt.NumbersRepetitionMode"
description: "Specifies whether and how DIAdem repeats the axis label in a polar axis system in DIAdem REPORT."
---

# IRepPolarRadialAxisInt.NumbersRepetitionMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: NumbersRepetitionMode for PolarRadialAxis

Specifies whether and how DIAdem repeats the axis label in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.NumbersRepetitionMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePolarAxisNumbersOnlyBeginning` | 0 | Only begin |
| `ePolarAxisNumbersBeginningAndEnd` | 1 | Begin and end |
| `ePolarAxisNumbersEvery090` | 2 | Every 90 degrees |
| `ePolarAxisNumbersEvery180` | 3 | Every 180 degrees |

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyRadialAxis = oMyPolarAxisSystem.RadialAxis
oMyRadialAxis.NumbersRepetitionMode = dd.ePolarAxisNumbersEvery090
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_NumbersRepetitionMode_IRepPolarRadialAxisInt.htm`*
