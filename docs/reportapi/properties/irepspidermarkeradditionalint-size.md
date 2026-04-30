---
title: "IRepSpiderMarkerAdditionalInt.Size"
description: "Specifies the size of the marker symbols as a percentage of the worksheet in a spider axis system in DIAdem REPORT."
---

# IRepSpiderMarkerAdditionalInt.Size

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Size for SpiderAdditionalMarker

Specifies the size of the marker symbols as a percentage of the worksheet in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Size
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

oMyMarker = oMyCurve.Shape.Extensions.Marker
oMyMarker.Type = dd.eMarkerSquare
oMyMarker.Size = 3
oMyMarker.Filling.UseCurveColor = True
oMyMarker.Line.Width = dd.eLineWidth0050
oMyMarker.Size = 3

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Size_IRepSpiderMarkerAdditionalInt.htm`*
