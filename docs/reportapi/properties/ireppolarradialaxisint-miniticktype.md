---
title: "IRepPolarRadialAxisInt.MiniTickType"
description: "Specifies the direction and the form of the miniticks for the Miniticks circle partition, in a polar display in DIAdem REPORT."
---

# IRepPolarRadialAxisInt.MiniTickType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MiniTickType for PolarRadialAxis

Specifies the direction and the form of the miniticks for the Miniticks circle partition, in a polar display in DIAdem REPORT.

## Signature

```python
obj.MiniTickType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePolarAxisMiniTickTypeBottom` | 0 | Miniticks bottom |
| `ePolarAxisMiniTickTypeTop` | 1 | Miniticks top |
| `ePolarAxisMiniTickTypeBothSides` | 2 | Miniticks top and bottom |
| `ePolarAxisMiniTickTypeCircle` | 3 | Miniticks as circles |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
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
oMyRadialAxis.MiniTickType = dd.ePolarAxisMiniTickTypeCircle
oMyMiniTickLine = oMyRadialAxis.MiniTickLine
oMyMiniTickLine.Color.ColorIndex = dd.eColorIndexYellow
oMyMiniTickLine.LineType = dd.eLineTypeSolid
oMyMiniTickLine.Width = dd.eLineWidth0100
oMyMiniTickLine.LineType = dd.eLineTypeSolid
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MiniTickType_IRepPolarRadialAxisInt.htm`*
