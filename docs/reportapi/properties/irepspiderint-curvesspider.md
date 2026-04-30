---
title: "IRepSpiderInt.CurvesSpider"
description: "Returns a collection of all curves in a spider axis system in DIAdem REPORT."
---

# IRepSpiderInt.CurvesSpider

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CurvesSpider for Spider

Returns a collection of all curves in a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.CurvesSpider
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

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_CurvesSpider_IRepSpiderInt.htm`*
