---
title: "IRepSpiderCurveInt.VisibleInLegend"
description: "Specifies whether DIAdem REPORT displays the curve legend in a spider axis system."
---

# IRepSpiderCurveInt.VisibleInLegend

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: VisibleInLegend for SpiderCurve

Specifies whether DIAdem REPORT displays the curve legend in a spider axis system.

## Signature

```python
obj.VisibleInLegend
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

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"
oMyCurve.Name = "MySpiderCurve"
oMyCurve.Enable = True
oMyAxisSystem.CurveLegend.Visible = True
oMyCurve.VisibleInLegend = False

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_VisibleInLegend_IRepSpiderCurveInt.htm`*
