---
title: "IRepSpiderCurveInt.Enable"
description: "Specifies whether DIAdem REPORT displays a curve in a spider axis system."
---

# IRepSpiderCurveInt.Enable

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Enable for SpiderCurve

Specifies whether DIAdem REPORT displays a curve in a spider axis system.

## Signature

```python
obj.Enable
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

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Enable_IRepSpiderCurveInt.htm`*
