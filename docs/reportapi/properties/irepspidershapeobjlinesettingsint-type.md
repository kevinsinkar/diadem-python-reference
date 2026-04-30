---
title: "IRepSpiderShapeObjLineSettingsInt.Type"
description: "Specifies the display type of a curve in the Line display mode in a spider axis system in DIAdem REPORT."
---

# IRepSpiderShapeObjLineSettingsInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for SpiderLineSettings

Specifies the display type of a curve in the Line display mode in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSpiderLineLinear` | 0 | Even |
| `eSpiderLineRounded` | 1 | Round |
| `eSpiderLineStaired` | 2 | Staired |

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

*Source: `ReportApi/properties/Report_property_Type_IRepSpiderShapeObjLineSettingsInt.htm`*
