---
title: "IRepSpiderCurveInt.LegendIconType"
description: "Specifies the display of the legend symbols in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCurveInt.LegendIconType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LegendIconType for SpiderCurve

Specifies the display of the legend symbols in a spider axis system in DIAdem REPORT.

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
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"
oMyCurve.Name = "MySpiderCurve"
oMyCurve.Enable = True

oMyAxisSystem.CurveLegend.Visible = True
oMyCurve.VisibleInLegend = False
oMyCurve.LegendIconType = dd.eLegendIconAllCurveStyles

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_LegendIconType_IRepSpiderCurveInt.htm`*
