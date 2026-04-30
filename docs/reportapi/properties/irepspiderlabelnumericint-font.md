---
title: "IRepSpiderLabelNumericInt.Font"
description: "Specifies the font for a scale label in a spider axis system in DIAdem REPORT."
---

# IRepSpiderLabelNumericInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for SpiderLabelNumeric

Specifies the font for a scale label in a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
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

*Source: `ReportApi/properties/Report_property_Font_IRepSpiderLabelNumericInt.htm`*
