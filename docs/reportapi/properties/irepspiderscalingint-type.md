---
title: "IRepSpiderScalingInt.Type"
description: "Specifies the scaling type of the standard axis in a spider axis system in DIAdem REPORT."
---

# IRepSpiderScalingInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for SpiderScaling

Specifies the scaling type of the standard axis in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSpiderScalingLinear` | 1 | Linear |
| `eSpiderScalingInverted` | 6 | Inverted |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPosition = oMyAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MyCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyCategorySettings = oMyAxisSystem.CategorySettings
oMyCategorySettings.Axis.Scaling.Type = dd.eSpiderScalingLinear

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepSpiderScalingInt.htm`*
