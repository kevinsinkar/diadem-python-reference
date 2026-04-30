---
title: "IRepSpiderInt.CurveLegend"
description: "Specifies the legend of a spider axis system in DIAdem REPORT."
---

# IRepSpiderInt.CurveLegend

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CurveLegend for Spider

Specifies the legend of a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.CurveLegend
```

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

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLineAndPoints, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyAxisSystem.CurveLegend.Visible = True

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_CurveLegend_IRepSpiderInt.htm`*
