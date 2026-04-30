---
title: "IRepSpiderMarkerAdditionalInt.Line"
description: "Specifies the properties of a marker line in a spider axis system in DIAdem REPORT."
---

# IRepSpiderMarkerAdditionalInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for SpiderAdditionalMarker

Specifies the properties of a marker line in a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
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

oMySpiderLineSettings = oMyCurve.Shape.Settings
oMySpiderLineSettings.Line.LineType = dd.eLineTypeDashed2
oMySpiderLineSettings.Type = dd.eSpiderLineStaired

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
<div class="SeeAlso">
<h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepSpiderMarkerAdditionalInt.htm`*
