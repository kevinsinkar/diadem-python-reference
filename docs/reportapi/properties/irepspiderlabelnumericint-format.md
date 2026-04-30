---
title: "IRepSpiderLabelNumericInt.Format"
description: "Specifies the Format definition of the scale labels in a spider axis system in DIAdem REPORT."
---

# IRepSpiderLabelNumericInt.Format

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Format for SpiderLabelNumeric

Specifies the Format definition of the scale labels in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Format
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

oMyAddLabel = oMyAxisSystem.CategorySettings.Axis.Numbers
oMyAddLabel.Font.Size = 1.5
oMyAddLabel.Format = "d"

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Format_IRepSpiderLabelNumericInt.htm`*
