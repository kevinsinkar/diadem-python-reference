---
title: "IRepPolarCurveInt.LegendIconType"
description: "Specifies the display of the legend symbols in a polar axis system in DIAdem REPORT."
---

# IRepPolarCurveInt.LegendIconType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LegendIconType for PolarCurve

Specifies the display of the legend symbols in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.LegendIconType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendIconAllCurveStyles` | 0 | Complete |
| `eLegendIconBasicCurveStylesOnly` | 1 | Only display type |
| `eLegendIconExtendedCurveStylesOnly` | 2 | Only extensions |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyPolarCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyCurve.Shape.Extensions.Marker.Type = dd.eMarkerCross
oMyLegend = oMyPolarAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyCurve.LegendIconType = dd.eLegendIconAllCurveStyles
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_LegendIconType_IRepPolarCurveInt.htm`*
