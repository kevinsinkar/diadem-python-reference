---
title: "IRepSpiderLabelAdditionalInt.ValueFormat"
description: "Specifies in a spider axis system in DIAdem REPORT the format instruction for the label of a curve with the associated values. You must assign the value TRUE to"
---

# IRepSpiderLabelAdditionalInt.ValueFormat

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ValueFormat for SpiderAdditionalLabel

Specifies in a spider axis system in DIAdem REPORT the format instruction for the label of a curve with the associated values. You must assign the value TRUE to the property ValueVisible in order to use the ValueFormat property.

## Signature

```python
obj.ValueFormat
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

oMyAddLabel = oMyCurve.Shape.Extensions.Label
oMyAddLabel.Font.Size = 1.5
oMyAddLabel.ValueVisible = True
oMyAddLabel.ValueFormat = "d"

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ValueFormat_IRepSpiderLabelAdditionalInt.htm`*
