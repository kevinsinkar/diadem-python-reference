---
title: "IRepSpiderLabelAdditionalInt.ValueVisible"
description: "Specifies whether DIAdem REPORT writes the coordinates at the curve points in a spider axis system with a curve in the Line and points display mode."
---

# IRepSpiderLabelAdditionalInt.ValueVisible

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ValueVisible for SpiderAdditionalLabel

Specifies whether DIAdem REPORT writes the coordinates at the curve points in a spider axis system with a curve in the Line and points display mode.

## Signature

```python
obj.ValueVisible
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

*Source: `ReportApi/properties/Report_property_ValueVisible_IRepSpiderLabelAdditionalInt.htm`*
